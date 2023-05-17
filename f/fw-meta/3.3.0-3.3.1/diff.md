# Comparing `tmp/fw_meta-3.3.0-py3-none-any.whl.zip` & `tmp/fw_meta-3.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14167 bytes, number of entries: 9
+Zip file size: 14277 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 fw_meta/__init__.py
 -rw-r--r--  2.0 unx      631 b- defN 80-Jan-01 00:00 fw_meta/aliases.py
 -rw-r--r--  2.0 unx     7728 b- defN 80-Jan-01 00:00 fw_meta/exports.py
--rw-r--r--  2.0 unx    20152 b- defN 80-Jan-01 00:00 fw_meta/imports.py
+-rw-r--r--  2.0 unx    20553 b- defN 80-Jan-01 00:00 fw_meta/imports.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_meta/py.typed
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_meta-3.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    10028 b- defN 80-Jan-01 00:00 fw_meta-3.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_meta-3.3.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      665 b- defN 16-Jan-01 00:00 fw_meta-3.3.0.dist-info/RECORD
-9 files, 40756 bytes uncompressed, 13039 bytes compressed:  68.0%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_meta-3.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10028 b- defN 80-Jan-01 00:00 fw_meta-3.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_meta-3.3.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      665 b- defN 16-Jan-01 00:00 fw_meta-3.3.1.dist-info/RECORD
+9 files, 41157 bytes uncompressed, 13149 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: fw_meta/imports.py
 Comment: 
 
 Filename: fw_meta/py.typed
 Comment: 
 
-Filename: fw_meta-3.3.0.dist-info/LICENSE
+Filename: fw_meta-3.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: fw_meta-3.3.0.dist-info/METADATA
+Filename: fw_meta-3.3.1.dist-info/METADATA
 Comment: 
 
-Filename: fw_meta-3.3.0.dist-info/WHEEL
+Filename: fw_meta-3.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: fw_meta-3.3.0.dist-info/RECORD
+Filename: fw_meta-3.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_meta/imports.py

```diff
@@ -264,14 +264,15 @@
     """Return validated field name and value as a tuple."""
     field, _ = validate_import_field(field)
     value = IMPORT_FIELD_LOADERS.get(field, load_any)(value)
     return field, value
 
 
 IMPORT_FIELD_LOADERS: t.Dict[str, t.Callable] = {
+    # TODO consider moving routing id under project
     "external_routing_id": load_any,
     "group._id": load_group_id,
     "group.label": load_cont_label,
     "project._id": load_cont_id,
     "project.label": load_cont_label,
     # TODO consider supporting project info updates in uploader
     # TODO validate and raise on empty info key (project.info.)
@@ -448,21 +449,23 @@
             "Exclude filters - if given, "
             "exclude files matching any of the exclude filters"
         ),
         example=["path=~meta.json"],
     )
     type: t.Optional[str] = Field(
         title=(
-            "Data type to import matching files as - if given, "
+            "Data type to import matching files with - if given, "
             "allows extracting additional metadata for known types"
         ),
         example="dicom",
     )
     group_by: t.Optional[str] = Field(
-        title="Group and process files together based on shared property", example="dir"
+        title="Group and process files together based on shared property",
+        readOnly=True,  # hide in inpus schemas for now
+        example="dir",
     )
     zip: t.Optional[bool] = Field(title="Import multiple grouped files zipped together")
     mappings: Mappings = Field(
         title="Metadata mapping patterns",
         example=[
             ("path", "{sub}/{ses}/{acq}/{file}"),
             ("path", "{file.info.original_path}"),
@@ -492,22 +495,27 @@
         # validate filters
         filt = ImportFilter(
             include=values.get("include"),
             exclude=values.get("exclude"),
         )
         values["include"] = [str(i) for i in filt.include]
         values["exclude"] = [str(e) for e in filt.exclude]
-        # validate type/group_by/zip
-        if values.get("type") == "dicom":
-            values.setdefault("group_by", "dir")
-            values.setdefault("zip", True)
-        if group_by := values.get("group_by"):
-            ImportTemplate(group_by)
-        if values.get("zip"):
-            assert group_by, "Zipping is only allowed when using group_by"
+        # autofill type/group_by/zip
+        if values.get("type") == "dicom" and values.get("zip") is None:
+            # auto-fill zip=true for type=dicom
+            values["zip"] = True
+        if values.get("zip") and values.get("group_by") is None:
+            # auto-fill group_by=dir for zip=true
+            values["group_by"] = "dir"
+        # validate group_by template
+        if values.get("group_by"):
+            ImportTemplate(values["group_by"])
+            # shouldn't get direct input from hidden field, but still auto-fill
+            if values.get("zip") is None:
+                values["zip"] = True  # pragma: no cover
         # validate patterns
         extractor = MetaExtractor(
             mappings=values.get("mappings"),
             defaults=values.get("defaults"),
             overrides=values.get("overrides"),
         )
         values["mappings"] = [(str(t), str(p)) for t, p in extractor.mappings]
```

## Comparing `fw_meta-3.3.0.dist-info/LICENSE` & `fw_meta-3.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_meta-3.3.0.dist-info/METADATA` & `fw_meta-3.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-meta
-Version: 3.3.0
+Version: 3.3.1
 Summary: Flywheel metadata extraction.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-meta
 License: MIT
 Keywords: Flywheel,DICOM,metadata,extract
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

