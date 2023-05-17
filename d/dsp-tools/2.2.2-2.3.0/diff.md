# Comparing `tmp/dsp_tools-2.2.2.tar.gz` & `tmp/dsp_tools-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-2.2.2.tar", max compression
+gzip compressed data, was "dsp_tools-2.3.0.tar", max compression
```

## Comparing `dsp_tools-2.2.2.tar` & `dsp_tools-2.3.0.tar`

### file list

```diff
@@ -1,58 +1,62 @@
--rw-r--r--   0        0        0    35149 2023-05-03 08:25:20.209025 dsp_tools-2.2.2/LICENSE
--rw-r--r--   0        0        0     4349 2023-05-03 08:25:20.221026 dsp_tools-2.2.2/docs/index.md
--rw-r--r--   0        0        0     5446 2023-05-03 08:25:20.221026 dsp_tools-2.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 08:25:20.221026 dsp_tools-2.2.2/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0    15624 2023-05-03 08:25:20.221026 dsp_tools-2.2.2/src/dsp_tools/dsp_tools.py
--rw-r--r--   0        0        0    81405 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/excel2xml.py
--rw-r--r--   0        0        0        0 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0      962 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/bitstream.py
--rw-r--r--   0        0        0     9766 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/connection.py
--rw-r--r--   0        0        0     3196 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     9472 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/group.py
--rw-r--r--   0        0        0    16923 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/helpers.py
--rw-r--r--   0        0        0     9702 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0    23044 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/listnode.py
--rw-r--r--   0        0        0      506 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/model.py
--rw-r--r--   0        0        0    19744 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/ontology.py
--rw-r--r--   0        0        0     2972 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/permission.py
--rw-r--r--   0        0        0    19120 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/project.py
--rw-r--r--   0        0        0     1930 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0    20998 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/propertyclass.py
--rw-r--r--   0        0        0     1896 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/propertyelement.py
--rw-r--r--   0        0        0    22008 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/resource.py
--rw-r--r--   0        0        0    34130 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/resourceclass.py
--rw-r--r--   0        0        0      419 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/set_encoder.py
--rw-r--r--   0        0        0      890 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/sipi.py
--rw-r--r--   0        0        0    27204 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/user.py
--rw-r--r--   0        0        0    34694 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/value.py
--rw-r--r--   0        0        0     2153 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/xmlallow.py
--rw-r--r--   0        0        0      747 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/xmlbitstream.py
--rw-r--r--   0        0        0      254 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/xmlerror.py
--rw-r--r--   0        0        0     1841 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/xmlpermission.py
--rw-r--r--   0        0        0     2371 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/xmlproperty.py
--rw-r--r--   0        0        0     8874 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/xmlresource.py
--rw-r--r--   0        0        0     2614 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/models/xmlvalue.py
--rw-r--r--   0        0        0     1488 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    23019 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    42584 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    32171 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0     2867 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0        0 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0    15112 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/excel_to_json_lists.py
--rw-r--r--   0        0        0     4891 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/excel_to_json_project.py
--rw-r--r--   0        0        0     7837 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/excel_to_json_properties.py
--rw-r--r--   0        0        0    10214 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/excel_to_json_resources.py
--rw-r--r--   0        0        0     1170 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/generate_templates.py
--rw-r--r--   0        0        0     3179 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/id_to_iri.py
--rw-r--r--   0        0        0    41148 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/project_create.py
--rw-r--r--   0        0        0     8048 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/project_create_lists.py
--rw-r--r--   0        0        0     4545 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/project_get.py
--rw-r--r--   0        0        0    18823 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/project_validate.py
--rw-r--r--   0        0        0     4231 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/rosetta.py
--rw-r--r--   0        0        0    12779 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0     6786 2023-05-03 08:25:20.225026 dsp_tools-2.2.2/src/dsp_tools/utils/stack_handling.py
--rw-r--r--   0        0        0    50393 2023-05-03 08:25:20.229026 dsp_tools-2.2.2/src/dsp_tools/utils/xml_upload.py
--rw-r--r--   0        0        0     5688 1970-01-01 00:00:00.000000 dsp_tools-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-17 07:10:03.642256 dsp_tools-2.3.0/LICENSE
+-rw-r--r--   0        0        0     4373 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/docs/index.md
+-rw-r--r--   0        0        0     5142 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0    20021 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/dsp_tools.py
+-rw-r--r--   0        0        0    82249 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/excel2xml.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/fast_xmlupload/__init__.py
+-rw-r--r--   0        0        0    29584 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/fast_xmlupload/process_files.py
+-rw-r--r--   0        0        0    14430 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/fast_xmlupload/upload_files.py
+-rw-r--r--   0        0        0     4157 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/fast_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0      962 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/bitstream.py
+-rw-r--r--   0        0        0     9766 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/connection.py
+-rw-r--r--   0        0        0     3203 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     9472 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/group.py
+-rw-r--r--   0        0        0    16923 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/helpers.py
+-rw-r--r--   0        0        0     9810 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0    23044 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/listnode.py
+-rw-r--r--   0        0        0      506 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/model.py
+-rw-r--r--   0        0        0    19744 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/ontology.py
+-rw-r--r--   0        0        0     2972 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/permission.py
+-rw-r--r--   0        0        0    19120 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/project.py
+-rw-r--r--   0        0        0     1930 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0    21101 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/propertyclass.py
+-rw-r--r--   0        0        0     1896 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/propertyelement.py
+-rw-r--r--   0        0        0    22008 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/resource.py
+-rw-r--r--   0        0        0    34520 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/resourceclass.py
+-rw-r--r--   0        0        0      419 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/set_encoder.py
+-rw-r--r--   0        0        0      890 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/sipi.py
+-rw-r--r--   0        0        0    27302 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/user.py
+-rw-r--r--   0        0        0    34694 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/value.py
+-rw-r--r--   0        0        0     2153 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlallow.py
+-rw-r--r--   0        0        0      747 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlbitstream.py
+-rw-r--r--   0        0        0      254 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlerror.py
+-rw-r--r--   0        0        0     1841 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlpermission.py
+-rw-r--r--   0        0        0     2371 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlproperty.py
+-rw-r--r--   0        0        0     8874 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlresource.py
+-rw-r--r--   0        0        0     2614 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlvalue.py
+-rw-r--r--   0        0        0     1488 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    23543 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    42584 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    32171 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0     2867 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0        0 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0    15112 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_lists.py
+-rw-r--r--   0        0        0     4891 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_project.py
+-rw-r--r--   0        0        0     7837 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_properties.py
+-rw-r--r--   0        0        0    10214 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_resources.py
+-rw-r--r--   0        0        0     1170 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/generate_templates.py
+-rw-r--r--   0        0        0     3179 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/id_to_iri.py
+-rw-r--r--   0        0        0    41148 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/project_create.py
+-rw-r--r--   0        0        0     8048 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/project_create_lists.py
+-rw-r--r--   0        0        0     4578 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/project_get.py
+-rw-r--r--   0        0        0    18834 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/project_validate.py
+-rw-r--r--   0        0        0     4265 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/rosetta.py
+-rw-r--r--   0        0        0    12854 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0     6838 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/stack_handling.py
+-rw-r--r--   0        0        0    50915 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/xml_upload.py
+-rw-r--r--   0        0        0     5725 1970-01-01 00:00:00.000000 dsp_tools-2.3.0/PKG-INFO
```

### Comparing `dsp_tools-2.2.2/LICENSE` & `dsp_tools-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/docs/index.md` & `dsp_tools-2.3.0/docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -45,26 +45,26 @@
   reads a project with its data model(s) from 
   a DSP server and writes it into a JSON file.
 - [`dsp-tools xmlupload`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#xmlupload) 
   uploads data from an XML file (bulk data import)
   and writes the mapping from internal IDs to IRIs into a local file.
 - [`dsp-tools excel2json`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2json) 
   creates an entire JSON project file from a folder with Excel files in it.
-  - [`dsp-tools excel2lists`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2lists)
-    creates the "lists" section of a JSON project file from one or several Excel files. 
-    The resulting section can be integrated into a JSON project file
-    and then be uploaded to a DSP server with `dsp-tools create`.
-  - [`dsp-tools excel2resources`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2resources)
-    creates the "resources" section of a JSON project file from an Excel file. 
-    The resulting section can be integrated into a JSON project file 
-    and then be uploaded to a DSP server with `dsp-tools create`.
-  - [`dsp-tools excel2properties`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2properties)
-    creates the "properties" section of a JSON project file from an Excel file. 
-    The resulting section can be integrated into a JSON project file 
-    and then be uploaded to a DSP server with `dsp-tools create`.
+    - [`dsp-tools excel2lists`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2lists)
+      creates the "lists" section of a JSON project file from one or several Excel files. 
+      The resulting section can be integrated into a JSON project file
+      and then be uploaded to a DSP server with `dsp-tools create`.
+    - [`dsp-tools excel2resources`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2resources)
+      creates the "resources" section of a JSON project file from an Excel file. 
+      The resulting section can be integrated into a JSON project file 
+      and then be uploaded to a DSP server with `dsp-tools create`.
+    - [`dsp-tools excel2properties`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2properties)
+      creates the "properties" section of a JSON project file from an Excel file. 
+      The resulting section can be integrated into a JSON project file 
+      and then be uploaded to a DSP server with `dsp-tools create`.
 - [`dsp-tools excel2xml`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2xml) 
   transforms a data source to XML 
   if it is already structured according to the DSP specifications.
 - [The module `excel2xml`](https://docs.dasch.swiss/latest/DSP-TOOLS/excel2xml-module) 
   provides helper methods that can be used in a Python script 
   to convert data from a tabular format into XML.
 - [`dsp-tools id2iri`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#id2iri)
```

### Comparing `dsp_tools-2.2.2/pyproject.toml` & `dsp_tools-2.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 
 [tool.poetry]
 name = "dsp-tools"
-version = "2.2.2"
+version = "2.3.0"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -24,50 +24,47 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 jsonpath-ng = "^1.5.3"
 argparse = "^1.4.0"
 lxml = "^4.9.2"
-requests = "^2.28.1"
+requests = "^2.30.0"
 jsonschema = "^4.17.3"
-openpyxl = "^3.0.10"
-networkx = "^2.8.8"
-pandas = "^1.5.2"
-xlrd = ">=1.0.0"            # without this, pandas raises an ImportError: Missing optional dependency 'xlrd'
-regex = "^2022.10.31"
+openpyxl = "^3.1.2"
+networkx = "^3.1.0"
+pandas = { version = "^2.0.1", extras = ["excel"] }  # extra package that contains xlrd that is necessary for reading old .xls Excel files
+regex = "^2023.5.5"
+docker = "^6.1.2"
 
 
 [tool.poetry.group.dev.dependencies]
-mkdocs = "^1.4.2"
-mkdocs-material = "^8.5.11"
-mkdocs-include-markdown-plugin = "^4.0.3"
-mypy = "^0.991"
-autopep8 = "^2.0.1"
-pytest = "^7.2.0"
-types-requests = "^2.28.11.7"
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.11"
+mkdocs-include-markdown-plugin = "^4.0.4"
+mypy = "^1.3.0"
+pylint = "^2.17.4"
+autopep8 = "^2.0.2"
+pytest = "^7.3.1"
+types-requests = "^2.30.0.0"
 types-lxml = "^2023.3.28"
-pylint = "^2.17.3"
-types-jsonschema = "^4.17.0.7"
-types-openpyxl = "^3.1.0.4"
-types-regex = "^2023.3.23.1"
+types-jsonschema = "^4.17.0.8"
+types-openpyxl = "^3.1.0.7"
+types-regex = "^2023.5.5.0"
 
 
 [tool.poetry.scripts]
 # definition of the entry point
 dsp-tools = "dsp_tools.dsp_tools:main"
 
 
 [tool.poetry-exec-plugin.commands]
 # plugin (https://github.com/keattang/poetry-exec-plugin) to define commands available for the developers
 # e.g. `poetry exec check-links`
 check-links = "markdown-link-validator ./docs -i \\.\\/assets\\/.+ -i .+github\\.com\\/dasch\\-swiss\\/dsp-tools\\/settings"
-# `mkdocs serve` can normally be executed without custom port. This is only necessary on machines where the standard
-# port is taken already
-docs-serve = "mkdocs serve --dev-addr=localhost:7979"
 
 
 [build-system]
 # Tells “frontend” build tools (like pip, build, or poetry) what “backend” build tool to use (e.g. setuptools, poetry).
 # The "backend" doesn't need to be installed. It will be installed by the "frontend" in a temporary, isolated
 # environment for use during the build process.
 requires = ["poetry-core"]
@@ -83,36 +80,34 @@
 
 [tool.autopep8]
 max_line_length = 150
 experimental = true
 
 
 [tool.mypy]
-ignore_missing_imports = true
+ignore_missing_imports = true              # TODO: deactivate this
 show_column_numbers = true
 strict = true
 exclude = [
-    "src/dsp_tools/models",           # TODO: activate this
-    "src/dsp_tools/import_scripts",   # TODO: activate this
-    "test/unittests",                 # TODO: activate this
-    "test/e2e",                       # TODO: activate this
+    "src/dsp_tools/models",                # TODO: activate this
+    "src/dsp_tools/import_scripts",        # TODO: activate this
+    "test/e2e",                            # TODO: activate this
 ]
 
 
 [tool.isort]
 multi_line_output = 3
 known_first_party = ["dsp_tools"]
 
 
 [tool.pylint.MASTER]
 ignore-paths = [
-    "src/dsp_tools/models/.*$",           # TODO: activate this
-    "src/dsp_tools/import_scripts/.*$",   # TODO: activate this
-    "test/unittests/.*$",                 # TODO: activate this
-    "test/e2e/.*$"                        # TODO: activate this
+    "src/dsp_tools/models/.*$",            # TODO: activate this
+    "src/dsp_tools/import_scripts/.*$",    # TODO: activate this
+    "test/e2e/.*$"                         # TODO: activate this
 ]
 suggestion-mode = true
 
 
 [tool.pylint.format]
 max-line-length = 150
 
@@ -141,10 +136,9 @@
     "too-many-arguments",                  # TODO: activate this
     "too-many-branches",                   # TODO: activate this
     "too-many-lines",                      # TODO: activate this
     "too-many-locals",                     # TODO: activate this
     "too-many-nested-blocks",              # TODO: activate this
     "too-many-return-statements",          # TODO: activate this
     "too-many-statements",                 # TODO: activate this
-    "bare-except",                         # TODO: activate this
     "consider-using-f-string",             # in excel2xml, strings with {} in it must be formatted
 ]
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/dsp_tools.py` & `dsp_tools-2.3.0/src/dsp_tools/dsp_tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import logging
 import logging.handlers
 import sys
 from importlib.metadata import version
 from pathlib import Path
 
 from dsp_tools.excel2xml import excel2xml
+from dsp_tools.fast_xmlupload.process_files import process_files
+from dsp_tools.fast_xmlupload.upload_files import upload_files
+from dsp_tools.fast_xmlupload.upload_xml import fast_xmlupload
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.excel_to_json_lists import (
     excel2lists,
     validate_lists_section_with_schema
 )
 from dsp_tools.utils.excel_to_json_project import excel2json
 from dsp_tools.utils.excel_to_json_properties import excel2properties
@@ -36,70 +39,110 @@
 
     Returns:
         parser
     """
     # help texts
     username_text = "username (e-mail) used for authentication with the DSP-API "
     password_text = "password used for authentication with the DSP-API "
-    url_text = "URL of the DSP server"
+    dsp_server_text = "URL of the DSP server"
     verbose_text = "print more information about the progress to the console"
+    sipi_text = "URL of the Sipi server"
 
     # default values
-    default_localhost = "http://0.0.0.0:3333"
+    default_dsp_api_url = "http://0.0.0.0:3333"
     default_user = "root@example.com"
     default_pw = "test"
+    default_sipi = "http://0.0.0.0:1024"
 
     # make a parser
     parser = argparse.ArgumentParser(description=f"DSP-TOOLS (version {version('dsp-tools')}, © {datetime.datetime.now().year} by DaSCH)")
     subparsers = parser.add_subparsers(title="Subcommands", description="Valid subcommands are", help="sub-command help")
 
     # create
     parser_create = subparsers.add_parser(
         name="create", 
         help="Create a project defined in a JSON project file on a DSP server. "
              "A project can consist of lists, groups, users, and ontologies (data models)."
     )
     parser_create.set_defaults(action="create")
-    parser_create.add_argument("-s", "--server", default=default_localhost, help=url_text)
+    parser_create.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
     parser_create.add_argument("-u", "--user", default=default_user, help=username_text)
     parser_create.add_argument("-p", "--password", default=default_pw, help=password_text)
     parser_create.add_argument("-V", "--validate-only", action="store_true", 
                                help="validate the JSON file without creating it on the DSP server")
     parser_create.add_argument("-l", "--lists-only", action="store_true", 
                                help="create only the lists (prerequisite: the project exists on the server)")
     parser_create.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_create.add_argument("-d", "--dump", action="store_true", help="dump test files for DSP-API requests")
     parser_create.add_argument("project_definition", help="path to the JSON project file")
 
     # get
     parser_get = subparsers.add_parser(name="get", help="Retrieve a project with its data model(s) from a DSP server and write it into a JSON file")
     parser_get.set_defaults(action="get")
-    parser_get.add_argument("-s", "--server", default=default_localhost, help=url_text)
+    parser_get.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
     parser_get.add_argument("-u", "--user", default=default_user, help=username_text)
     parser_get.add_argument("-p", "--password", default=default_pw, help=password_text)
     parser_get.add_argument("-P", "--project", help="shortcode, shortname or IRI of the project", required=True)
     parser_get.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_get.add_argument("project_definition", help="path to the file the project should be written to")
 
     # xmlupload
     parser_upload = subparsers.add_parser(name="xmlupload", help="Upload data defined in an XML file to a DSP server")
     parser_upload.set_defaults(action="xmlupload")
-    parser_upload.add_argument("-s", "--server", default=default_localhost, help="URL of the DSP server where DSP-TOOLS sends the data to")
+    parser_upload.add_argument("-s", "--server", default=default_dsp_api_url, help="URL of the DSP server where DSP-TOOLS sends the data to")
     parser_upload.add_argument("-u", "--user", default=default_user, help=username_text)
     parser_upload.add_argument("-p", "--password", default=default_pw, help=password_text)
-    parser_upload.add_argument("-S", "--sipi", default="http://0.0.0.0:1024", 
+    parser_upload.add_argument("-S", "--sipi", default=default_sipi, 
                                help="URL of the SIPI server where DSP-TOOLS sends the multimedia files to")
     parser_upload.add_argument("-i", "--imgdir", default=".", help="folder from where the paths in the <bitstream> tags are evaluated")
     parser_upload.add_argument("-I", "--incremental", action="store_true", 
                                help="The links in the XML file point to IRIs (on the server) instead of IDs (in the same XML file).")
     parser_upload.add_argument("-V", "--validate", action="store_true", help="validate the XML file without uploading it")
     parser_upload.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_upload.add_argument("-m", "--metrics", action="store_true", help="write metrics into a 'metrics' folder")
     parser_upload.add_argument("xmlfile", help="path to the XML file containing the data")
 
+    # process-files
+    parser_process_files = subparsers.add_parser(
+        name="process-files",
+        help="For internal use only: process all files referenced in an XML file"
+    )
+    parser_process_files.set_defaults(action="process-files")
+    parser_process_files.add_argument("--input-dir", help="path to the input directory where the files should be read from")
+    parser_process_files.add_argument("--output-dir", help="path to the output directory where the processed/transformed files should be written to")
+    parser_process_files.add_argument("--nthreads", type=int, default=None, help="number of threads to use")
+    parser_process_files.add_argument("xml_file", help="path to XML file containing the data")
+
+    # upload-files
+    parser_upload_files = subparsers.add_parser(
+        name="upload-files",
+        help="For internal use only: upload already processed files"
+    )
+    parser_upload_files.set_defaults(action="upload-files")
+    parser_upload_files.add_argument("-f", "--pkl-file", help="path to pickle file written by 'process-files'")
+    parser_upload_files.add_argument("-d", "--processed-dir", help="path to the directory with the processed files")
+    parser_upload_files.add_argument("-n", "--nthreads", type=int, default=4, help="number of threads to use")
+    parser_upload_files.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
+    parser_upload_files.add_argument("-S", "--sipi-url", default=default_sipi, help=sipi_text)
+    parser_upload_files.add_argument("-u", "--user", default=default_user, help=username_text)
+    parser_upload_files.add_argument("-p", "--password", default=default_pw, help=password_text)
+
+    # fast-xmlupload
+    parser_fast_xmlupload_files = subparsers.add_parser(
+        name="fast-xmlupload",
+        help="For internal use only: create resources with already uploaded files"
+    )
+    parser_fast_xmlupload_files.set_defaults(action="fast-xmlupload")
+    parser_fast_xmlupload_files.add_argument("-f", "--pkl-file", help="path to pickle file written by 'process-files'")
+    parser_fast_xmlupload_files.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
+    parser_fast_xmlupload_files.add_argument("-S", "--sipi-url", default=default_sipi, help=sipi_text)
+    parser_fast_xmlupload_files.add_argument("-u", "--user", default=default_user, help=username_text)
+    parser_fast_xmlupload_files.add_argument("-p", "--password", default=default_pw, help=password_text)
+    parser_fast_xmlupload_files.add_argument("xml_file", help="path to XML file containing the data")
+
     # excel2json
     parser_excel2json = subparsers.add_parser(
         name="excel2json",
         help="Create an entire JSON project file from a folder containing the required Excel files"
     )
     parser_excel2json.set_defaults(action="excel2json")
     parser_excel2json.add_argument("excelfolder", help="path to the folder containing the Excel files")
@@ -153,16 +196,15 @@
     parser_id2iri.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_id2iri.add_argument("xmlfile", help="path to the XML file containing the data to be replaced")
     parser_id2iri.add_argument("mapping", help="path to the JSON file containing the mapping of IDs to IRIs")
 
     # startup DSP stack
     parser_stackup = subparsers.add_parser(name="start-stack", help="Run a local instance of DSP-API and DSP-APP")
     parser_stackup.set_defaults(action="start-stack")
-    parser_stackup.add_argument("--max_file_size", type=int, 
-                                help="max. multimedia file size allowed by SIPI, in MB (default: 250, max: 100'000)")
+    parser_stackup.add_argument("--max_file_size", type=int, help="max. multimedia file size allowed by SIPI, in MB (default: 250, max: 100'000)")
     parser_stackup.add_argument("--prune", action="store_true", help="execute 'docker system prune' without asking")
     parser_stackup.add_argument("--no-prune", action="store_true", help="don't execute 'docker system prune' (and don't ask)")
 
     # shutdown DSP-API
     parser_stackdown = subparsers.add_parser(
         name="stop-stack", 
         help="Shut down the local instance of DSP-API and DSP-APP, and delete all data in it"
@@ -171,49 +213,56 @@
 
     # create template repo with minimal JSON and XML files
     parser_template = subparsers.add_parser(
         name="template", 
         help="Create a template repository with a minimal JSON and XML file"
     )
     parser_template.set_defaults(action="template")
-    
+
     # clone rosetta
     parser_rosetta = subparsers.add_parser(
         name="rosetta", 
         help="Clone the most up to data rosetta repository, create the data model and upload the data"
     )
     parser_rosetta.set_defaults(action="rosetta")
 
     return parser
 
 
 def call_requested_action(
     user_args: list[str], 
-    parser: argparse.ArgumentParser
+    parser: argparse.ArgumentParser,
+    logger: logging.Logger
 ) -> bool:
     """
     With the help of the parser, parse the user arguments and call the appropriate method of DSP-TOOLS.
 
     Args:
         user_args: list of arguments passed by the user from the command line
         parser: parser to parse the user arguments
+        logger: the logger for this module
 
     Raises:
         BaseError from the called methods
         UserError from the called methods
         unexpected errors from the called methods and underlying libraries
     
     Returns:
         success status
     """
     args = parser.parse_args(user_args)
     if not hasattr(args, "action"):
         parser.print_help(sys.stderr)
         sys.exit(1)
-    elif args.action == "create":
+    
+    logger.info("*****************************************************************************************")
+    logger.info(f"***Called DSP-TOOLS action '{args.action}' from command line with these parameters: {args}")
+    logger.info("*****************************************************************************************")
+    
+    if args.action == "create":
         if args.lists_only:
             if args.validate_only:
                 success = validate_lists_section_with_schema(path_to_json_project_file=args.project_definition)
                 print("'Lists' section of the JSON project file is syntactically correct and passed validation.")
             else:
                 _, success = create_lists(
                     project_file_as_path_or_parsed=args.project_definition,
@@ -253,16 +302,44 @@
                 server=args.server,
                 user=args.user,
                 password=args.password,
                 imgdir=args.imgdir,
                 sipi=args.sipi,
                 verbose=args.verbose,
                 incremental=args.incremental,
-                save_metrics=args.metrics
+                save_metrics=args.metrics,
+                preprocessing_done=False
             )
+
+    elif args.action == "process-files":
+        success = process_files(
+            input_dir=args.input_dir,
+            output_dir=args.output_dir,
+            xml_file=args.xml_file,
+            nthreads=args.nthreads
+        )
+    elif args.action == "upload-files":
+        success = upload_files(
+            pkl_file=args.pkl_file,
+            dir_with_processed_files=args.processed_dir,
+            nthreads=args.nthreads,
+            user=args.user,
+            password=args.password,
+            dsp_url=args.server,
+            sipi_url=args.sipi_url
+        )
+    elif args.action == "fast-xmlupload":
+        success = fast_xmlupload(
+            xml_file=args.xml_file,
+            pkl_file=args.pkl_file,
+            user=args.user,
+            password=args.password,
+            dsp_url=args.server,
+            sipi_url=args.sipi_url
+        )
     elif args.action == "excel2json":
         success = excel2json(
             data_model_files=args.excelfolder,
             path_to_output_file=args.project_definition
         )
     elif args.action == "excel2lists":
         _, success = excel2lists(
@@ -303,17 +380,18 @@
         success = stop_stack()
     elif args.action == "template":
         success = generate_template_repo()
     elif args.action == "rosetta":
         success = upload_rosetta()
     else:
         success = False
+        print(f"ERROR: Unknown action '{args.action}'")
+        logger.error(f"Unknown action '{args.action}'")
 
     return success
-    
 
 
 def main() -> None:
     """Main entry point of the program as referenced in pyproject.toml"""
     logging.basicConfig(
         format="{asctime}   {filename: <20} {levelname: <8} {message}",
         style="{",
@@ -322,21 +400,27 @@
             logging.handlers.RotatingFileHandler(
                 filename=Path.home() / Path(".dsp-tools") / "logging.log",
                 maxBytes=3*1024*1024,
                 backupCount=1
             )
         ]
     )
+    logger = logging.getLogger(__name__)
     
     parser = make_parser()
     try:
-        success = call_requested_action(user_args=sys.argv[1:], parser=parser)
+        success = call_requested_action(
+            user_args=sys.argv[1:], 
+            parser=parser, 
+            logger=logger
+        )
     except UserError as err:
         print(err.message)
         sys.exit(1)
     # let BaseError and all unexpected errors escalate, so that a stack trace is printed
 
     if not success: 
         sys.exit(1)
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/excel2xml.py` & `dsp_tools-2.3.0/src/dsp_tools/excel2xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,20 @@
 import pandas as pd
 import regex
 from lxml import etree
 from lxml.builder import E  # pylint: disable=no-name-in-module
 
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.helpers import DateTimeStamp
-from dsp_tools.models.propertyelement import PropertyElement
+# explicitly export PropertyElement, so that API users can import it from this module 
+# (see https://mypy.readthedocs.io/en/stable/command_line.html#cmdoption-mypy-no-implicit-reexport)
+# doing this requires silencing the corresponding pylint warning 
+# (see https://pylint.readthedocs.io/en/latest/user_guide/messages/convention/useless-import-alias.html)
+from dsp_tools.models.propertyelement import \
+    PropertyElement as PropertyElement  # pylint: disable=useless-import-alias
 from dsp_tools.models.value import UriValue
 from dsp_tools.utils.shared import (
     check_notna,
     simplify_name,
     validate_xml_against_schema
 )
 
@@ -396,15 +401,18 @@
     Examples:
         >>> resource = make_resource(...)
         >>> resource.append(make_text_prop(...))
         >>> root.append(resource)
 
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#describing-resources-with-the-resource-element
     """
-
+    if not check_notna(label):
+        warnings.warn(f"WARNING: Your resource's label looks suspicious (resource with id '{id}' and label '{label}'")
+    if not check_notna(id):
+        warnings.warn(f"WARNING: Your resource's id looks suspicious (resource with id '{id}' and label '{label}'")
     kwargs = {
         "label": label,
         "restype": restype,
         "id": id,
         "permissions": permissions,
         "nsmap": xml_namespace_map
     }
@@ -1269,16 +1277,19 @@
             content = etree.tostring(value_, encoding="unicode")
             # ... insert text at the very end of the string, and add an ending tag to the previously single <text/> tag ...
             content = re.sub(r"/>$", f">{val.value}</text>", content)
             # ... try to parse it again
             try:
                 value_ = etree.fromstring(content)
             except etree.XMLSyntaxError:
-                raise BaseError("The XML tags contained in a richtext property (encoding=xml) must be well-formed. "
-                                "The special characters <, > and & are only allowed to construct a tag.") from None
+                raise BaseError(
+                    "The XML tags contained in a richtext property (encoding=xml) must be well-formed. "
+                    "The special characters <, > and & are only allowed to construct a tag."
+                    f"The error occurred in resource {calling_resource}, property {name}"
+                ) from None
         prop_.append(value_)
 
     return prop_
 
 
 def make_time_prop(
     name: str,
@@ -1873,15 +1884,15 @@
             resource_restype = row.get("restype")
             if not check_notna(resource_restype):
                 raise BaseError(f"Missing restype for resource {resource_id}")
             if check_notna(row.get("ark")) and check_notna(row.get("iri")):
                 raise BaseError(f"Both ARK and IRI were provided for resource '{resource_label}' ({resource_id}). The ARK will override the IRI.")
             # previous resource is finished, now a new resource begins. in all cases (except for
             # the very first iteration), a previous resource exists. if it exists, append it to root.
-            if resource:
+            if resource is not None:
                 root.append(resource)
             kwargs_resource = {
                 "label": resource_label,
                 "permissions": resource_permissions,
                 "id": resource_id
             }
             if check_notna(row.get("ark")):
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/bitstream.py` & `dsp_tools-2.3.0/src/dsp_tools/models/bitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/connection.py` & `dsp_tools-2.3.0/src/dsp_tools/models/connection.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/exceptions.py` & `dsp_tools-2.3.0/src/dsp_tools/models/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         original_error_msg_from_api: The original error message that DSP-API returns (only applicable if the error comes from DSP-API)
         reason_from_api_response: The reason for the failure that DSP-API returns (only applicable if the error comes from DSP-API)
         api_route: The route that was called (only applicable if the error comes from DSP-API)
     """
     message: str
     status_code: Optional[int]
     json_content_of_api_response: Optional[str]
-    original_error_msg_from_api: Optional[str]
+    original_error_msg_from_api: Optional[str] = None
     reason_from_api_response: Optional[str]
     api_route: Optional[str]
 
     def __init__(
         self, 
         message: str, 
         status_code: Optional[int] = None,
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/group.py` & `dsp_tools-2.3.0/src/dsp_tools/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/helpers.py` & `dsp_tools-2.3.0/src/dsp_tools/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/langstring.py` & `dsp_tools-2.3.0/src/dsp_tools/models/langstring.py`

 * *Files 10% similar despite different names*

```diff
@@ -176,30 +176,30 @@
                 if lmap.get(key.lower()) is None:
                     raise BaseError('Invalid language string "' + key + '"!')
                 return self._langstrs.get(lmap[key.lower()])
 
     def items(self):
         return self._langstrs.items()
 
-    def isEmpty(self):
+    def isEmpty(self) -> bool:
         return not (bool(self._langstrs) or bool(self._simplestring))
 
-    def empty(self):
+    def empty(self) -> None:
         self._simplestring = None
         self._langstrs = {}
 
-    def toJsonObj(self):
+    def toJsonObj(self) -> Optional[Union[str, list[dict[str, str]]]]:
         if self.isEmpty():
             return None
         if self._simplestring is not None:
             return self._simplestring
         else:
             return list(map(lambda a: {'language': a[0].value, 'value': a[1] if a[1] else "-"}, self._langstrs.items()))
 
-    def toJsonLdObj(self):
+    def toJsonLdObj(self) -> Optional[Union[str, list[dict[str, str]]]]:
         if self.isEmpty():
             return None
         if self._simplestring is not None:
             return self._simplestring
         else:
             return [{'@language': a[0].value, '@value': a[1]} for a in self._langstrs.items()]
             # return list(map(lambda a: {'@language': a[0].value, '@value': a[1]}, self._langstrs.items()))
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/listnode.py` & `dsp_tools-2.3.0/src/dsp_tools/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/ontology.py` & `dsp_tools-2.3.0/src/dsp_tools/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/permission.py` & `dsp_tools-2.3.0/src/dsp_tools/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/project.py` & `dsp_tools-2.3.0/src/dsp_tools/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/projectContext.py` & `dsp_tools-2.3.0/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/propertyclass.py` & `dsp_tools-2.3.0/src/dsp_tools/models/propertyclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,14 +428,16 @@
         if self.object:
             property["name"] = self.name
         if self.superproperties:
             superprops = []
             for sc in self.superproperties:
                 superprops.append(context.reduce_iri(sc, shortname))
             property["super"] = superprops
+        if self.subject:
+            property["subject"] = context.reduce_iri(self.subject, shortname)
         if self.object:
             property["object"] = context.reduce_iri(self.object, shortname)
         if self.label:
             property["labels"] = self.label.createDefinitionFileObj()
         if self.comment:
             property["comments"] = self.comment.createDefinitionFileObj()
         if self.gui_element:
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/propertyelement.py` & `dsp_tools-2.3.0/src/dsp_tools/models/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/resource.py` & `dsp_tools-2.3.0/src/dsp_tools/models/resource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/resourceclass.py` & `dsp_tools-2.3.0/src/dsp_tools/models/resourceclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,15 +273,20 @@
 
     def delete(self, last_modification_date: DateTimeStamp) -> DateTimeStamp:
         raise BaseError("Cannot remove a single property from a class!")
         # ToDo: Check with Ben if we could add this feature...
 
     def createDefinitionFileObj(self, context: Context, shortname: str):
         cardinality = {}
-        if self._ptype == HasProperty.Ptype.other:
+        if self._ptype == HasProperty.Ptype.other or self.property_id in [
+            "knora-api:isSequenceOf", 
+            "knora-api:hasSequenceBounds", 
+            "knora-api:isPartOf", 
+            "knora-api:seqnum"
+        ]:
             cardinality["propname"] = context.reduce_iri(self._property_id, shortname)
             cardinality["cardinality"] = self._cardinality.value
             if self._gui_order is not None:
                 cardinality["gui_order"] = self._gui_order
         return cardinality
 
     def print(self, offset: int = 0):
@@ -770,38 +775,42 @@
 
     def delete(self, last_modification_date: DateTimeStamp) -> DateTimeStamp:
         result = self._con.delete(
             ResourceClass.ROUTE + '/' + quote_plus(self._id) + '?lastModificationDate=' + str(last_modification_date))
         return DateTimeStamp(result['knora-api:lastModificationDate'])
 
     def createDefinitionFileObj(self, context: Context, shortname: str, skiplist: list[str]):
-        resource = {
-            "name": self._name,
-            "labels": self._label.createDefinitionFileObj(),
-        }
-        if self._comment:
-            resource["comments"] = self._comment.createDefinitionFileObj()
+        resource = {"name": self._name}
         if self._superclasses:
             if len(self._superclasses) > 1:
                 superclasses = []
                 for sc in self._superclasses:
                     superclasses.append(context.reduce_iri(sc, shortname))
             else:
                 superclasses = context.reduce_iri(self._superclasses[0], shortname)
             resource["super"] = superclasses
+        resource["labels"] = self._label.createDefinitionFileObj()
+        if self._comment:
+            resource["comments"] = self._comment.createDefinitionFileObj()
         if self._has_properties:
             cardinalities = []
             for pid, hp in self._has_properties.items():
                 if hp.property_id in skiplist:
                     continue
-                if hp.ptype == HasProperty.Ptype.other:
+                if hp.ptype == HasProperty.Ptype.other or hp.property_id in [
+                    "knora-api:isSequenceOf", 
+                    "knora-api:hasSequenceBounds", 
+                    "knora-api:isPartOf", 
+                    "knora-api:seqnum"
+                ]:
                     cardinalities.append(hp.createDefinitionFileObj(context, shortname))
             if cardinalities:
                 resource["cardinalities"] = cardinalities
 
+
         return resource
 
     def print(self, offset: int = 0):
         blank = ' '
         print(f'{blank:>{offset}}Resource Class Info')
         print(f'{blank:>{offset + 2}}Name:            {self._name}')
         print(f'{blank:>{offset + 2}}Ontology prefix: {self._ontology_id}')
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/sipi.py` & `dsp_tools-2.3.0/src/dsp_tools/models/sipi.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/user.py` & `dsp_tools-2.3.0/src/dsp_tools/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -692,39 +692,42 @@
         res.reverse()
         return res
 
     def createDefinitionFileObj(
         self,
         con: Connection,
         proj_shortname: str,
-        proj_shortcode: str
+        proj_iri: str
     ) -> dict[str, Union[str, list[str], None]]:
-        user: dict[str, Union[str, list[str], None]] = {
+        user: dict[str, Union[str, list[str], bool, None]] = {
             "username": self.username,
             "email": self.email,
             "givenName": self.givenName,
             "familyName": self.familyName,
             "password": "",
         }
         if self.lang:
             user["lang"] = self.lang.value
         groups = list()
         for group_iri in self._in_groups:
             group_info = con.get(f'/admin/groups/{urllib.parse.quote_plus(group_iri)}')
             if 'group' in group_info and 'name' in group_info['group']:
                 groupname = group_info['group']['name']
                 groups.append(f'{proj_shortname}:{groupname}')
+        if self.sysadmin:
+            groups.append("SystemAdmin")
         user["groups"] = groups
         user["projects"] = list()
         for proj, is_admin in self._in_projects.items():
-            if proj_shortcode in proj:
+            if proj == proj_iri:
                 if is_admin:
                     user["projects"].append(f"{proj_shortname}:admin")
                 else:
                     user["projects"].append(f"{proj_shortname}:member")
+        user["status"] = self.status
         return user
 
     def print(self) -> None:
         """
         Prin user info to stdout
 
         :return: None
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/value.py` & `dsp_tools-2.3.0/src/dsp_tools/models/value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/xmlallow.py` & `dsp_tools-2.3.0/src/dsp_tools/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/xmlbitstream.py` & `dsp_tools-2.3.0/src/dsp_tools/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/xmlpermission.py` & `dsp_tools-2.3.0/src/dsp_tools/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/xmlproperty.py` & `dsp_tools-2.3.0/src/dsp_tools/models/xmlproperty.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/xmlresource.py` & `dsp_tools-2.3.0/src/dsp_tools/models/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/models/xmlvalue.py` & `dsp_tools-2.3.0/src/dsp_tools/models/xmlvalue.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-2.3.0/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-2.3.0/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-2.3.0/src/dsp_tools/resources/schema/data.xsd`

 * *Files 1% similar despite different names*

#### Comparing `dsp_tools-2.2.2/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-2.3.0/src/dsp_tools/resources/schema/data.xsd`

```diff
@@ -352,15 +352,21 @@
         <xs:element name="resptr-prop" type="resptrprop_type" minOccurs="0" maxOccurs="unbounded"/>
         <xs:element name="time-prop" type="timeprop_type" minOccurs="0" maxOccurs="unbounded"/>
         <xs:element name="decimal-prop" type="decimalprop_type" minOccurs="0" maxOccurs="unbounded"/>
         <xs:element name="uri-prop" type="uriprop_type" minOccurs="0" maxOccurs="unbounded"/>
         <xs:element name="boolean-prop" type="booleanprop_type" minOccurs="0" maxOccurs="unbounded"/>
       </xs:choice>
     </xs:sequence>
-    <xs:attribute name="label" type="xs:string" use="required"/>
+    <xs:attribute name="label" use="required">
+      <xs:simpleType>
+        <xs:restriction base="xs:string">
+          <xs:minLength value="1"/>
+        </xs:restriction>
+      </xs:simpleType>
+    </xs:attribute>
     <xs:attribute name="restype" type="xs:string" use="required"/>
     <xs:attribute name="id" type="xs:ID" use="required"/>
     <xs:attribute name="permissions" type="xs:NCName" use="optional"/>
     <xs:attribute name="iri" type="xs:string" use="optional"/>
     <xs:attribute name="ark" type="xs:string" use="optional"/>
     <xs:attribute name="creation_date" type="xs:dateTime" use="optional"/>
   </xs:complexType>
@@ -475,9 +481,17 @@
       <xs:selector xpath="./permissions"/>
       <xs:field xpath="@id"/>
     </xs:key>
     <xs:keyref name="permissionsIdref" refer="permissionsId">
       <xs:selector xpath="resource"/>
       <xs:field xpath="@permissions"/>
     </xs:keyref>
+    <xs:unique name="IRI_attribute_of_resource_must_be_unique">
+      <xs:selector xpath=".//*"/>
+      <xs:field xpath="@iri"/>
+    </xs:unique>
+    <xs:unique name="ARK_attribute_of_resource_must_be_unique">
+      <xs:selector xpath=".//*"/>
+      <xs:field xpath="@ark"/>
+    </xs:unique>
   </xs:element>
 </xs:schema>
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-2.3.0/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/resources/schema/project.json` & `dsp_tools-2.3.0/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-2.3.0/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-2.3.0/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-2.3.0/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
       - knora-net
     environment:
       - TZ=Europe/Zurich
       - ADMIN_PASSWORD=test
       - JVM_ARGS=-Xmx3G
 
   sipi:
-    image: daschswiss/knora-sipi:28.1.2  # on the verge of every deployment (fortnightly), take the same tag as DSP-API
+    image: daschswiss/knora-sipi:28.2.0  # on the verge of every deployment (fortnightly), take the same tag as DSP-API
     ports:
       - "1024:1024"
     volumes:
       - .:/docker
     networks:
       - knora-net
     environment:
@@ -42,15 +42,15 @@
       - SIPI_WEBAPI_HOSTNAME=api
       - SIPI_WEBAPI_PORT=3333
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_HOST=0.0.0.0
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_PORT=3333
     command: --config=/docker/sipi.docker-config.lua
 
   api:
-    image: daschswiss/knora-api:28.1.2  # on the verge of every deployment (fortnightly),
+    image: daschswiss/knora-api:28.2.0  # on the verge of every deployment (fortnightly),
                                         # take the tag of https://hub.docker.com/r/daschswiss/knora-api/tags
                                         # that corresponds to the version on https://admin.staging.dasch.swiss/help
                                         # (see also https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json)
     depends_on:
       - sipi
       - db
     ports:
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/excel_to_json_lists.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/excel_to_json_project.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/excel_to_json_properties.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_properties.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/excel_to_json_resources.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_resources.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/generate_templates.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/generate_templates.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/id_to_iri.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/id_to_iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/project_create.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/project_create.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/project_create_lists.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/project_create_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/project_get.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/project_get.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import re
-from typing import Optional
+from typing import Any
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.group import Group
 from dsp_tools.models.listnode import ListNode
 from dsp_tools.models.ontology import Ontology
 from dsp_tools.models.project import Project
@@ -46,42 +46,44 @@
     project = project.read()
 
     project_obj = project.createDefinitionFileObj()
 
     # get groups
     if verbose:
         print("Getting groups...")
-    groups_obj = []
-    groups: Optional[list[Group]] = Group.getAllGroupsForProject(con=con, proj_iri=str(project.id))
+    groups_obj: list[dict[str, Any]] = []
+    groups = Group.getAllGroupsForProject(con=con, proj_iri=str(project.id))
     if groups:
         for group in groups:
             groups_obj.append(group.createDefinitionFileObj())
             if verbose:
                 print(f"\tGot group '{group.name}'")
     project_obj["groups"] = groups_obj
 
     # get users
     if verbose:
         print("Getting users...")
-    users_obj = []
+    users_obj: list[dict[str, Any]] = []
     users = User.getAllUsersForProject(con=con, proj_shortcode=str(project.shortcode))
     if users:
         for usr in users:
             users_obj.append(usr.createDefinitionFileObj(
-                con=con, proj_shortname=str(project.shortname), proj_shortcode=str(project.shortcode)
+                con=con, 
+                proj_shortname=str(project.shortname), 
+                proj_iri=str(project.id)
             ))
             if verbose:
                 print(f"\tGot user '{usr.username}'")
         project_obj["users"] = users_obj
 
     # get the lists
     if verbose:
         print("Getting lists...")
-    list_obj = []
-    list_roots: Optional[list[ListNode]] = ListNode.getAllLists(con=con, project_iri=project.id)
+    list_obj: list[dict[str, Any]] = []
+    list_roots = ListNode.getAllLists(con=con, project_iri=project.id)
     if list_roots:
         for list_root in list_roots:
             complete_list = list_root.getAllNodes()
             list_obj.append(complete_list.createDefinitionFileObj())
             if verbose:
                 print(f"\tGot list '{list_root.name}'")
     project_obj["lists"] = list_obj
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/project_validate.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/project_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,15 +397,15 @@
     for start, cards in dependencies.items():
         for edge, targets in cards.items():
             for target in targets:
                 graph.add_edge(start, target, edge)
 
     # find elements of circles that have a cardinality of "1" or "1-n"
     errors: set[tuple[str, str]] = set()
-    circles = list(nx.cycles.simple_cycles(graph))
+    circles = list(nx.algorithms.cycles.simple_cycles(graph))
     for circle in circles:
         for index, resource in enumerate(circle):
             target = circle[(index+1) % len(circle)]
             prop = ""
             for _property, targets in dependencies[resource].items():
                 if target in targets:
                     prop = _property
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/rosetta.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/rosetta.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,16 @@
         server="http://0.0.0.0:3333",
         user="root@example.com",
         password="test",
         imgdir=str(rosetta_folder),
         sipi="http://0.0.0.0:1024",
         verbose=False,
         incremental=False,
-        save_metrics=False
+        save_metrics=False,
+        preprocessing_done=False
     )
     return success
 
 
 def upload_rosetta() -> bool:
     """
     This method clones https://github.com/dasch-swiss/082E-rosetta-scripts
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/shared.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     _validate_xml_tags_in_text_properties(doc)    
 
     logger.info("The XML file is syntactically correct and passed validation.")
     print("The XML file is syntactically correct and passed validation.")
     return True
 
 
-def _validate_xml_tags_in_text_properties(doc: etree._ElementTree[Any]) -> bool:
+def _validate_xml_tags_in_text_properties(doc: Union[etree._ElementTree[etree._Element], etree._Element]) -> bool:
     """
     Makes sure that there are no XML tags in simple texts.
     This can only be done with a regex, 
     because even if the simple text contains some XML tags, 
     the simple text itself is not valid XML that could be parsed.
     The extra challenge is that lxml transforms 
     "pebble (&lt;2cm) and boulder (&gt;20cm)" into 
@@ -175,16 +175,16 @@
     
     # then: make the test
     resources_with_illegal_xml_tags = list()
     for text in doc_without_namespace.findall(path="resource/text-prop/text"):
         if text.attrib["encoding"] == "utf8":
             if regex.search(r'<([a-zA-Z/"]+|[^\s0-9].*[^\s0-9])>', str(text.text)) or len(list(text.iterchildren())) > 0:
                 sourceline = f" line {text.sourceline}: " if text.sourceline else " "
-                propname = text.getparent().attrib["name"]
-                resname = text.getparent().getparent().attrib["id"]
+                propname = text.getparent().attrib["name"]           # type: ignore
+                resname = text.getparent().getparent().attrib["id"]  # type: ignore
                 resources_with_illegal_xml_tags.append(f" -{sourceline}resource '{resname}', property '{propname}'")
     if resources_with_illegal_xml_tags:
         err_msg = "XML-tags are not allowed in text properties with encoding=utf8. The following resources of your XML file violate this rule:\n" 
         err_msg += "\n".join(resources_with_illegal_xml_tags)
         logger.error(err_msg, exc_info=True)
         raise UserError(err_msg)
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/stack_handling.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/stack_handling.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     docker_path_of_distribution = importlib.resources.files("dsp_tools").joinpath("resources/start-stack")
     for file in docker_path_of_distribution.iterdir():
         with importlib.resources.as_file(file) as f:
             file_path = Path(f)
         shutil.copy(file_path, docker_path_of_user / file.name)
 
     # get sipi.docker-config.lua
-    commit_of_used_api_version = "6375a719a326705ee274ebfff12770b9f1dc14d7"      # gitleaks:allow
+    commit_of_used_api_version = "d6bae7ff5e6b6a635982c14f21ca4e69e298a312"      # gitleaks:allow
     url_prefix = f"https://github.com/dasch-swiss/dsp-api/raw/{commit_of_used_api_version}/"
     docker_config_lua_text = requests.get(f"{url_prefix}sipi/config/sipi.docker-config.lua", timeout=5).text
     if max_file_size:
         max_post_size_regex = r"max_post_size ?= ?[\'\"]\d+M[\'\"]"
         if not re.search(max_post_size_regex, docker_config_lua_text):
             raise BaseError("Unable to set max_file_size. Please try again without this flag.")
         docker_config_lua_text = re.sub(max_post_size_regex, f"max_post_size = '{max_file_size}M'", docker_config_lua_text)
@@ -67,15 +67,15 @@
 
     # wait until fuseki is up (same behaviour as dsp-api/webapi/scripts/wait-for-db.sh)
     for _ in range(360):
         try:
             response = requests.get(url="http://0.0.0.0:3030/$/server", auth=("admin", "test"), timeout=5)
             if response.ok:
                 break
-        except:
+        except Exception:  # pylint: disable=broad-exception-caught
             time.sleep(1)
         time.sleep(1)
 
     # inside fuseki, create the "knora-test" repository
     # (same behaviour as dsp-api/webapi/target/docker/stage/opt/docker/scripts/fuseki-init-knora-test.sh)
     repo_template = requests.get(f"{url_prefix}webapi/scripts/fuseki-repository-config.ttl.template", timeout=5).text
     repo_template = repo_template.replace("@REPOSITORY@", "knora-test")
```

### Comparing `dsp_tools-2.2.2/src/dsp_tools/utils/xml_upload.py` & `dsp_tools-2.3.0/src/dsp_tools/utils/xml_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         print(f"\nWARNING: Could not upload the following resources: {failed_uploads}\n")
         logger.warning(f"Could not upload the following resources: {failed_uploads}")
         success = False
     if metrics:
         os.makedirs("metrics", exist_ok=True)
         df = pd.DataFrame(metrics)
         df.to_csv(f"metrics/{metrics_filename}")
+        print(f"Total time of xmlupload: {sum(int(record.duration_ms) for record in metrics) / 1000:.1f} seconds")
 
     return success
 
 
 def _remove_circular_references(resources: list[XMLResource], verbose: bool) -> \
         tuple[list[XMLResource],
               dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
@@ -440,29 +441,31 @@
     server: str, 
     user: str, 
     password: str, 
     imgdir: str, 
     sipi: str, 
     verbose: bool,
     incremental: bool, 
-    save_metrics: bool
+    save_metrics: bool,
+    preprocessing_done: bool
 ) -> bool:
     """
     This function reads an XML file and imports the data described in it onto the DSP server.
 
     Args:
         input_file: path to the XML file or parsed ElementTree
         server: the DSP server where the data should be imported
         user: the user (e-mail) with which the data should be imported
         password: the password of the user with which the data should be imported
         imgdir: the image directory
         sipi: the sipi instance to be used
         verbose: verbose option for the command, if used more output is given to the user
         incremental: if set, IRIs instead of internal IDs are expected as resource pointers
         save_metrics: if true, saves time measurements into a "metrics" folder in the current working directory
+        preprocessing_done: if set, all multimedia files referenced in the XML file must already be on the server
 
     Raises:
         BaseError or UserError in case of permanent network or software failure
         UserError if the XML file is invalid
     
     Returns:
         True if all resources could be uploaded without errors; False if one of the resources could not be
@@ -500,18 +503,18 @@
         raise UserError("Unable to retrieve project context from DSP server") from None
     sipi_server = Sipi(sipi, con.get_token())
 
     # make Python object representations of the XML file
     resources: list[XMLResource] = []
     permissions: dict[str, XmlPermission] = {}
     for child in root:
-        if child.tag == "permissions":  # type: ignore
+        if child.tag == "permissions":
             permission = XmlPermission(child, proj_context)
             permissions[permission.id] = permission
-        elif child.tag == "resource":  # type: ignore
+        elif child.tag == "resource":
             resources.append(XMLResource(child, default_ontology))
 
     # get the project information and project ontology from the server
     try:
         res_inst_factory = try_network_action(lambda: ResourceInstanceFactory(con, shortcode))
     except BaseError:
         logger.error(f"A project with shortcode {shortcode} could not be found on the DSP server", exc_info=True)
@@ -543,15 +546,15 @@
     id2iri_mapping: dict[str, str] = {}
     failed_uploads: list[str] = []
     nonapplied_resptr_props = {}
     nonapplied_xml_texts = {}
     try:
         id2iri_mapping, failed_uploads, metrics = _upload_resources(
             resources, imgdir, sipi_server, permissions_lookup, resclass_name_2_type, id2iri_mapping, con,
-            failed_uploads, metrics
+            failed_uploads, metrics, preprocessing_done
         )
         if stashed_xml_texts:
             nonapplied_xml_texts = _upload_stashed_xml_texts(verbose, id2iri_mapping, con, stashed_xml_texts) 
         if stashed_resptr_props:
             nonapplied_resptr_props = _upload_stashed_resptr_props(verbose, id2iri_mapping, con, stashed_resptr_props)
         if nonapplied_resptr_props or nonapplied_xml_texts:
             logger.error("Some stashed resptrs or XML texts could not be reapplied to their resources on the DSP server.")
@@ -589,15 +592,16 @@
     imgdir: str,
     sipi_server: Sipi,
     permissions_lookup: dict[str, Permissions],
     resclass_name_2_type: dict[str, type],
     id2iri_mapping: dict[str, str],
     con: Connection,
     failed_uploads: list[str],
-    metrics: list[MetricRecord]
+    metrics: list[MetricRecord],
+    preprocessing_done: bool
 ) -> tuple[dict[str, str], list[str], list[MetricRecord]]:
     """
     Iterates through all resources and tries to upload them to DSP.
     If a temporary exception occurs, the action is repeated until success,
     and if a permanent exception occurs, the resource is skipped.
 
     Args:
@@ -612,15 +616,17 @@
         metrics: list with the metric records collected until now (gets filled during the upload)
 
     Returns:
         id2iri_mapping, failed_uploads, metrics
     """
 
     # If there are multimedia files: calculate their total size
-    bitstream_all_sizes_mb = [Path(Path(imgdir) / Path(res.bitstream.value)).stat().st_size / 1000000 if res.bitstream else 0.0 for res in resources]
+    bitstream_all_sizes_mb = [Path(Path(imgdir) / Path(res.bitstream.value)).stat().st_size / 1000000
+                              if res.bitstream and not preprocessing_done else 0.0
+                              for res in resources]
     if sum(bitstream_all_sizes_mb) > 0:
         bitstream_size_total_mb = round(sum(bitstream_all_sizes_mb), 1)
         bitstream_size_uploaded_mb = 0.0
         print(f"This xmlupload contains multimedia files with a total size of {bitstream_size_total_mb} MB.")
         logger.info(f"This xmlupload contains multimedia files with a total size of {bitstream_size_total_mb} MB.")
     else:  # make Pylance happy
         bitstream_size_total_mb = 0.0
@@ -633,15 +639,17 @@
         bitstream_duration_ms = None
         resource_iri = resource.iri
         if resource.ark:
             resource_iri = _convert_ark_v0_to_resource_iri(resource.ark)
 
         # in case of a multimedia resource: upload the multimedia file
         resource_bitstream = None
-        if resource.bitstream:
+        if preprocessing_done and resource.bitstream:
+            resource_bitstream = resource.get_bitstream(resource.bitstream.value, permissions_lookup)
+        elif resource.bitstream:
             try:
                 bitstream_start = datetime.now()
                 filetype = Path(resource.bitstream.value).suffix[1:]
                 img: Optional[dict[Any, Any]] = try_network_action(
                     sipi_server.upload_bitstream,
                     filepath=str(Path(imgdir) / Path(resource.bitstream.value))
                 )
```

### Comparing `dsp_tools-2.2.2/PKG-INFO` & `dsp_tools-2.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 2.2.2
+Version: 2.3.0
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
+Requires-Dist: docker (>=6.1.2,<7.0.0)
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: networkx (>=2.8.8,<3.0.0)
-Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
-Requires-Dist: pandas (>=1.5.2,<2.0.0)
-Requires-Dist: regex (>=2022.10.31,<2023.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: xlrd (>=1.0.0)
+Requires-Dist: networkx (>=3.1.0,<4.0.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
+Requires-Dist: pandas[excel] (>=2.0.1,<3.0.0)
+Requires-Dist: regex (>=2023.5.5,<2024.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
 Project-URL: Documentation, https://docs.dasch.swiss/latest/DSP-TOOLS/
 Project-URL: Repository, https://github.com/dasch-swiss/dsp-tools
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/dsp-tools.svg)](https://badge.fury.io/py/dsp-tools)
 
 # DSP-TOOLS documentation
@@ -75,26 +75,26 @@
   reads a project with its data model(s) from 
   a DSP server and writes it into a JSON file.
 - [`dsp-tools xmlupload`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#xmlupload) 
   uploads data from an XML file (bulk data import)
   and writes the mapping from internal IDs to IRIs into a local file.
 - [`dsp-tools excel2json`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2json) 
   creates an entire JSON project file from a folder with Excel files in it.
-  - [`dsp-tools excel2lists`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2lists)
-    creates the "lists" section of a JSON project file from one or several Excel files. 
-    The resulting section can be integrated into a JSON project file
-    and then be uploaded to a DSP server with `dsp-tools create`.
-  - [`dsp-tools excel2resources`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2resources)
-    creates the "resources" section of a JSON project file from an Excel file. 
-    The resulting section can be integrated into a JSON project file 
-    and then be uploaded to a DSP server with `dsp-tools create`.
-  - [`dsp-tools excel2properties`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2properties)
-    creates the "properties" section of a JSON project file from an Excel file. 
-    The resulting section can be integrated into a JSON project file 
-    and then be uploaded to a DSP server with `dsp-tools create`.
+    - [`dsp-tools excel2lists`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2lists)
+      creates the "lists" section of a JSON project file from one or several Excel files. 
+      The resulting section can be integrated into a JSON project file
+      and then be uploaded to a DSP server with `dsp-tools create`.
+    - [`dsp-tools excel2resources`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2resources)
+      creates the "resources" section of a JSON project file from an Excel file. 
+      The resulting section can be integrated into a JSON project file 
+      and then be uploaded to a DSP server with `dsp-tools create`.
+    - [`dsp-tools excel2properties`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2properties)
+      creates the "properties" section of a JSON project file from an Excel file. 
+      The resulting section can be integrated into a JSON project file 
+      and then be uploaded to a DSP server with `dsp-tools create`.
 - [`dsp-tools excel2xml`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2xml) 
   transforms a data source to XML 
   if it is already structured according to the DSP specifications.
 - [The module `excel2xml`](https://docs.dasch.swiss/latest/DSP-TOOLS/excel2xml-module) 
   provides helper methods that can be used in a Python script 
   to convert data from a tabular format into XML.
 - [`dsp-tools id2iri`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#id2iri)
```

