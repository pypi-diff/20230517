# Comparing `tmp/fw_storage-2.1.6-py3-none-any.whl.zip` & `tmp/fw_storage-2.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 37820 bytes, number of entries: 24
+Zip file size: 37976 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      511 b- defN 80-Jan-01 00:00 fw_storage/__init__.py
 -rw-r--r--  2.0 unx    18182 b- defN 80-Jan-01 00:00 fw_storage/config.py
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 fw_storage/errors.py
--rw-r--r--  2.0 unx      963 b- defN 80-Jan-01 00:00 fw_storage/fileinfo.py
+-rw-r--r--  2.0 unx     1676 b- defN 80-Jan-01 00:00 fw_storage/fileinfo.py
 -rw-r--r--  2.0 unx     1016 b- defN 80-Jan-01 00:00 fw_storage/filters.py
 -rw-r--r--  2.0 unx     1013 b- defN 80-Jan-01 00:00 fw_storage/future/__init__.py
 -rw-r--r--  2.0 unx    11816 b- defN 80-Jan-01 00:00 fw_storage/future/base.py
 -rw-r--r--  2.0 unx     4652 b- defN 80-Jan-01 00:00 fw_storage/future/errors.py
 -rw-r--r--  2.0 unx       36 b- defN 80-Jan-01 00:00 fw_storage/future/types/__init__.py
 -rw-r--r--  2.0 unx    12755 b- defN 80-Jan-01 00:00 fw_storage/future/types/fs.py
 -rw-r--r--  2.0 unx     3934 b- defN 80-Jan-01 00:00 fw_storage/future/utils.py
@@ -15,12 +15,12 @@
 -rw-r--r--  2.0 unx       28 b- defN 80-Jan-01 00:00 fw_storage/types/__init__.py
 -rw-r--r--  2.0 unx     6844 b- defN 80-Jan-01 00:00 fw_storage/types/az.py
 -rw-r--r--  2.0 unx    13338 b- defN 80-Jan-01 00:00 fw_storage/types/dicom.py
 -rw-r--r--  2.0 unx     7996 b- defN 80-Jan-01 00:00 fw_storage/types/dicomweb.py
 -rw-r--r--  2.0 unx      140 b- defN 80-Jan-01 00:00 fw_storage/types/fs.py
 -rw-r--r--  2.0 unx     4861 b- defN 80-Jan-01 00:00 fw_storage/types/gs.py
 -rw-r--r--  2.0 unx     6374 b- defN 80-Jan-01 00:00 fw_storage/types/s3.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_storage-2.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     4013 b- defN 80-Jan-01 00:00 fw_storage-2.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_storage-2.1.6.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1924 b- defN 16-Jan-01 00:00 fw_storage-2.1.6.dist-info/RECORD
-24 files, 109352 bytes uncompressed, 34736 bytes compressed:  68.2%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_storage-2.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4013 b- defN 80-Jan-01 00:00 fw_storage-2.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_storage-2.1.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1925 b- defN 16-Jan-01 00:00 fw_storage-2.1.7.dist-info/RECORD
+24 files, 110066 bytes uncompressed, 34892 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: fw_storage/types/gs.py
 Comment: 
 
 Filename: fw_storage/types/s3.py
 Comment: 
 
-Filename: fw_storage-2.1.6.dist-info/LICENSE
+Filename: fw_storage-2.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: fw_storage-2.1.6.dist-info/METADATA
+Filename: fw_storage-2.1.7.dist-info/METADATA
 Comment: 
 
-Filename: fw_storage-2.1.6.dist-info/WHEEL
+Filename: fw_storage-2.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: fw_storage-2.1.6.dist-info/RECORD
+Filename: fw_storage-2.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_storage/fileinfo.py

```diff
@@ -1,10 +1,11 @@
 """File-info module."""
 import dataclasses
 import typing as t
+from pathlib import Path
 
 
 @dataclasses.dataclass(frozen=True)
 class FileInfo:
     """FileInfo dataclass yielded from storage.ls() calls.
 
     Path is unique and relative to the storage prefix. Slots minimize memory
@@ -20,14 +21,35 @@
     modified: t.Optional[t.Union[int, float]]
 
     def asdict(self) -> t.Dict:
         """Return as a dictionary."""
         # TODO performance-test this and improve as needed
         return dataclasses.asdict(self)  # pragma: no cover
 
-    def dict(self) -> t.Dict:
+    def dict(self) -> t.Dict:  # pragma: no cover
         """Future compatibility."""
-        return self.asdict()  # pragma: no cover
+        return self.asdict()
 
-    def __str__(self) -> str:
+    @property
+    def dir(self) -> str:  # pragma: no cover
+        """Return the directory name of this path."""
+        dirname = str(Path(self.path).parent)
+        return "" if dirname == "." else dirname
+
+    @property
+    def name(self) -> str:  # pragma: no cover
+        """Return the base filename of this path."""
+        return Path(self.path).name
+
+    @property
+    def stem(self) -> str:  # pragma: no cover
+        """Return the filename stem without any extension suffix."""
+        return Path(self.path).stem
+
+    @property
+    def ext(self) -> str:  # pragma: no cover
+        """Return the extension of this path."""
+        return Path(self.path).suffix.lstrip(".")
+
+    def __str__(self) -> str:  # pragma: no cover
         """Return the path string."""
-        return self.path  # pragma: no cover
+        return self.path
```

## fw_storage/future/base.py

 * *Ordering differences only*

```diff
@@ -97,35 +97,14 @@
 
 
 class Item(BaseModel):
     """Storage item representing an individual file/blob/etc."""
 
     path: str
 
-    @property
-    def dir(self) -> str:
-        """Return the directory name of this path."""
-        dirname = str(Path(self.path).parent)
-        return "" if dirname == "." else dirname
-
-    @property
-    def name(self) -> str:
-        """Return the base filename of this path."""
-        return Path(self.path).name
-
-    @property
-    def stem(self) -> str:
-        """Return the filename stem without any extension suffix."""
-        return Path(self.path).stem
-
-    @property
-    def ext(self) -> str:
-        """Return the extension of this path."""
-        return Path(self.path).suffix.lstrip(".")
-
     def __str__(self) -> str:
         """Return string representation."""
         return self.path
 
     # STORAGE FILEINFO INTERFACE BACKWARDS COMPATIBILITY
     # TODO deprecation warning (when most of future is implemented)
 
@@ -257,14 +236,35 @@
     """File item with common attrs of files or blobs."""
 
     size: int
     ctime: t.Union[int, float, None]
     mtime: t.Union[int, float, None]
     hash: str
 
+    @property
+    def dir(self) -> str:
+        """Return the directory name of this path."""
+        dirname = str(Path(self.path).parent)
+        return "" if dirname == "." else dirname
+
+    @property
+    def name(self) -> str:
+        """Return the base filename of this path."""
+        return Path(self.path).name
+
+    @property
+    def stem(self) -> str:
+        """Return the filename stem without any extension suffix."""
+        return Path(self.path).stem
+
+    @property
+    def ext(self) -> str:
+        """Return the extension of this path."""
+        return Path(self.path).suffix.lstrip(".")
+
     # STORAGE ITEM (OLD FILEINFO) INTERFACE BACKWARDS COMPATIBILITY
     # TODO deprecation warning (when most of future is implemented)
 
     @property
     def created(self):
         """Backwards compatibility only."""
         return self.ctime
```

## Comparing `fw_storage-2.1.6.dist-info/LICENSE` & `fw_storage-2.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_storage-2.1.6.dist-info/METADATA` & `fw_storage-2.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-storage
-Version: 2.1.6
+Version: 2.1.7
 Summary: Unified storage interface.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-storage
 License: MIT
 Keywords: Flywheel,file,object,storage
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

## Comparing `fw_storage-2.1.6.dist-info/RECORD` & `fw_storage-2.1.7.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 fw_storage/__init__.py,sha256=v36QDeDLZJv7Sj2zXEZ6s0YIxuz42A9OA8boUEFnPvk,511
 fw_storage/config.py,sha256=VNKq8MNQ4dudrJqU6tBmEx8s5kmOdqKhliFvnvncx_s,18182
 fw_storage/errors.py,sha256=HD92V9ebpmsILbhf239XRSmwmO_-WHiOEuYdCUnL1V4,113
-fw_storage/fileinfo.py,sha256=6Xwu3OewGiua6DYFGObNJIAJvF1yiFfdC9sbaJ1nqgc,963
+fw_storage/fileinfo.py,sha256=dukS4wGSyy-uH_OmFNYViCnrTY_agPldoYs8wUuyTIo,1676
 fw_storage/filters.py,sha256=P3C1oGw1q6UoNEbHiSr-xdi_jumosSKOQgsulZ2GGaA,1016
 fw_storage/future/__init__.py,sha256=TWyZ7CFeCDO4_uiiT6gLJhE-SP8Ie7bNsCB3vUSbv2U,1013
-fw_storage/future/base.py,sha256=x7nPuhlbUoobeii8mz6CBV3lfxPJC4L6ph5fBOC6XyU,11816
+fw_storage/future/base.py,sha256=GsXb5vvvmm1iSn9ErM_djNjSKEbsIeqzCxw39m96lDo,11816
 fw_storage/future/errors.py,sha256=tE-wb4n_X8-v2zaU5KpoPlQVfDaDhazOpjLmNU45cw0,4652
 fw_storage/future/types/__init__.py,sha256=zOnfjDtMpINsVdYFikGbvjIf_FVnfPpm-DanhqDrLjo,36
 fw_storage/future/types/fs.py,sha256=xxs7p7Q6AQRwPALAg5Ds386yHh9k2cDe1HFtLKKrUWo,12755
 fw_storage/future/utils.py,sha256=JLVhxqSsA0uyNMbhPKyEQoJ3FVYoqLyjyO3bfeO4OOk,3934
 fw_storage/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fw_storage/storage.py,sha256=WgEySgS8f4Mjlx1lthDwtpfQ5XWVgTutQGCXPz1e-b8,7677
 fw_storage/types/__init__.py,sha256=TT2pfyY-AMuKb4FZduNbVbmWTBRyEC3autb1QbdHE24,28
 fw_storage/types/az.py,sha256=J2KbT9ugvTpLfAZg4BX0lDLK4i2lM8EYisyAnj9tVG4,6844
 fw_storage/types/dicom.py,sha256=XUSFsdSGTyNb8a6-K2H0jvztzj5lT5FmuGHt8pi_SCI,13338
 fw_storage/types/dicomweb.py,sha256=NR9E-csPgznASouwIdokukAxGPKCPRobhz80e4-z_v0,7996
 fw_storage/types/fs.py,sha256=Cz_GGrS_e11m9SvDgdjJkMf-VMI0s5DKUJZp0bWSegM,140
 fw_storage/types/gs.py,sha256=lQRo9qz0EHf3YmPO7LzLBFYEGkwqhmlVtxwF2T9EISI,4861
 fw_storage/types/s3.py,sha256=MMelCfrbaNZbZqGPBj9mt_Cdyhrbeq-ObYmmC4bM1G4,6374
-fw_storage-2.1.6.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
-fw_storage-2.1.6.dist-info/METADATA,sha256=450JDD27NHbwCyykZOt4FtJt6Gb9QzpoutYNbK6wbhk,4013
-fw_storage-2.1.6.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fw_storage-2.1.6.dist-info/RECORD,,
+fw_storage-2.1.7.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
+fw_storage-2.1.7.dist-info/METADATA,sha256=M4SGrmNECRk6Bcp758GIF6dxnoAy5xx0lQsniBpyt80,4013
+fw_storage-2.1.7.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fw_storage-2.1.7.dist-info/RECORD,,
```

